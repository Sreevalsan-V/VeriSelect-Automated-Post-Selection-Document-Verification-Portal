# VeriSelect-Automated-Post-Selection-Document-Verification-Portal

{
  "photo_url": "https://storage.example.com/photos/sreevalsan.jpg",

  "identity_verification": {
    "aadhaar": {
      "verified": true,
      "reason": "Matched with UIDAI data"
    },
    "pan": {
      "verified": false,
      "reason": "Name mismatch with Aadhaar"
    },
    "passport": {
      "verified": true,
      "reason": "All details consistent"
    },
    "summary": {
      "overall_identity_verified": false,
      "reason": "PAN verification failed"
    }
  },

  "education_verification": {
    "tenth_certificate": {
      "verified": true,
      "reason": "Matched with board record"
    },
    "twelfth_certificate": {
      "verified": true,
      "reason": "All subjects consistent"
    },
    "degree_certificate": {
      "verified": false,
      "reason": "University record not found in DigiLocker"
    },
    "summary": {
      "overall_education_verified": false,
      "reason": "Degree not verified"
    }
  },

  "certifications_verification": {
    "coursera_certificate": {
      "verified": true,
      "reason": "Verified via Coursera public API"
    },
    "udemy_certificate": {
      "verified": false,
      "reason": "Certificate ID invalid or revoked"
    },
    "summary": {
      "overall_certification_verified": false,
      "reason": "One invalid certificate found"
    }
  },

  "employment_verification": {
    "previous_company": {
      "company_name": "TechNova Systems",
      "hr_contact_email": "hr@technova.in",
      "hr_contact_number": "+91-9876543210",
      "verified": true,
      "reason": "Confirmed by HR via API"
    },
    "summary": {
      "overall_employment_verified": true
    }
  },

  "final_verification_summary": {
    "overall_verified": false,
    "failed_segments": [
      "Identity (PAN)",
      "Education (Degree)",
      "Certifications (Udemy)"
    ],
    "remarks": "Candidate verified except for degree and PAN mismatch"
  }
}
