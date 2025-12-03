erDiagram
	direction TB
	NewCandidate {

	}

	Purpose_of_Apply {

	}

	Information_Collection_Section {
		string YourAddress  "Please enter your Address"  
		string InterviewDetailsSection  ""  
		string Avalabilitysection  ""  
		string Profilesection  ""  
		string Skills  "Tell us about your skills"  
		string Comments  ""  
		string ActivitesSection  ""  
		string Joblistsection  ""  
		float Payslip  ""  
		string Referral  ""  
		string DiarySection  ""  
		string CommunicationHistorySection  ""  
		String AuditTraiSEction  ""  
		string RecordProperties  ""  
		string CandidateworkRefrence  ""  
		String CustomExit  ""  
	}

	Generalinfo {
		string(99) FirstName  " First name."  
		string LastName  "Last name "  
		Date DOB  ""  
		int Contact_information  ""  
	}

	OUtlook {
		string Email  "Registration Linnk"  
	}

	Already_Registered {

	}

	Appendix {
		String AssociatedDocummentes  ""  
		String CompetencyRequirement  ""  
		String VersionControl  ""  
	}

	NewCandidate||--||OUtlook:"receives"
	Purpose_of_Apply}|--||NewCandidate:"Application for job "
	Generalinfo|o--|{Information_Collection_Section:" Recording Process "
	Information_Collection_Section}|--||Appendix:" storing info and Docs "
	OUtlook}|--|{Generalinfo:"login  "
	Already_Registered||--|{Generalinfo:" Info Collection "
    