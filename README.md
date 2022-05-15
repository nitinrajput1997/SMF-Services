# SMF-Services

![](/smfService.png)

There are two main services as follows:  

1. Nsmf_PDUSession Service<br />
    It manages the PDU Session. It has includes functions:<br />
    1. Nsmf_PDUSession_Create<br />
      Used to create a new PDU session in H(home)-SMF.<br />
    2. Nsmf_PDUSession_Update<br />
      Used between the V(visitor)-SMF and H-SMF in roaming scenarios to update the established PDU session.<br />
    4. Nsmf_PDUSession_Release<br />
      Used in roaming scenario bu V-SMF to request thw H-SMF to release PDU Session.<br />
    5. Nsmf_PDUSession_StatusNotify<br />
      Used in roaming scenario by the H-SMF to notify V-SMF.<br />
    6. Nsmf_PDUSession_CreateSMContext<br />
      Used by AMF to creates an AMF-SMF association to support a PDU Session.<br />
    7. Nsmf_PDUSession_UpdateSMContext<br />
      Used by AMF to updates an AMF-SMF association to support a PDU Session.<br />
    8. Nsmf_PDUSession_ReleaseSMContext<br />
      Used by AMF to release the AMF-SMF association.<br />
    9. Nsmf_PDUSession_SMContextStatusNotify<br />
      Used by SMF to notify the AMF when PDU Session is released.<br />
    10. Nsmf_PDUSession_ContextRequest<br />
      Used by AMF to fetch the SM-Context during handover to EPS.<br />

2. Nsmf_EventExposure Service<br />
   It is used to subscribe and get notified about eventd related to PDU session. Exposes the information about PDU session related events like: UE address or Prefix change, PDU session release, User Plane path change, PLMN chnages. Event filter can be used.
