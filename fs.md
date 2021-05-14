            //find property in IBS
            //check property in CRM

            //logic need check date in Crm and IBS, make sure Property AddressId is correct

            //if not exists
            //create address based on property address
            //create property and set addressId


            //find latest tenancy in IBS
            //find the mapping tenancy in CRM
            //if not exists
            //create tenancy and get tenancyId
            //else
            //get tenancyId from CRM

            //get all the persons from IBS CustomerHistoric --need IBSPersonRef,PersonType,StartDate,EndDate

            //get all persons can be mapped from crm
            //if current tenancy exists
                // find out all missing tenant details
                    // check their existing tenant details, need set endDate if exists(otherwise, provide warning for multiple active tenancies for person
                    // create missing tenancies
                // update existing tenant details, check surename, ninumber, personstartdate, personendate
            
            //else create missing person tenancies
                //check their previous tenant details, need set endDate if exists(otherwise, provide warning for multiple active tenancies for person

            // note : may need to remove incorrect person tenancies details from crm
                    // need to check to make sure tenant is not garage etc when fetching tenancies
