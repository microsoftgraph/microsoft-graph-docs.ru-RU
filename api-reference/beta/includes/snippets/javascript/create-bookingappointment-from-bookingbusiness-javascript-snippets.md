---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e05416ae4168531164d976e58253e029b3cc223
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingAppointment = {
    '@odata.type':'#microsoft.graph.bookingAppointment',
    customerEmailAddress: 'jordanm@contoso.com',
    customerLocation: {
        '@odata.type':'#microsoft.graph.location',
        address: {
            '@odata.type':'#microsoft.graph.physicalAddress',
            city: 'Buffalo',
            countryOrRegion: 'USA',
            postalCode: '98052',
            postOfficeBox: null,
            state: 'NY',
            street: '123 First Avenue',
            'type@odata.type':'#microsoft.graph.physicalAddressType',
            type: null
        },
        coordinates: null,
        displayName: 'Customer',
        locationEmailAddress: null,
        'locationType@odata.type':'#microsoft.graph.locationType',
        locationType: null,
        locationUri: null,
        uniqueId: null,
        'uniqueIdType@odata.type':'#microsoft.graph.locationUniqueIdType',
        uniqueIdType: null
    },
    customerName: 'Jordan Miller',
    customerNotes: 'Please be on time.',
    customerPhone: '213-555-0199',
    end: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-01T12:30:00.0000000+00:00',
        timeZone: 'UTC'
    },
    invoiceAmount: 10.0,
    invoiceDate: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-01T12:30:00.0000000+00:00',
        timeZone: 'UTC'
    },
    invoiceId: '1001',
    'invoiceStatus@odata.type':'#microsoft.graph.bookingInvoiceStatus',
    invoiceStatus: 'open',
    invoiceUrl: 'theInvoiceUrl',
    optOutOfCustomerEmail: false,
    postBuffer: 'PT10M',
    preBuffer: 'PT5M',
    price: 10.0,
    'priceType@odata.type':'#microsoft.graph.bookingPriceType',
    priceType: 'fixedPrice',
    'reminders@odata.type':'#Collection(microsoft.graph.bookingReminder)',
    reminders: [
        {
            '@odata.type':'#microsoft.graph.bookingReminder',
            message: 'This service is tomorrow',
            offset: 'P1D',
            'recipients@odata.type':'#microsoft.graph.bookingReminderRecipients',
            recipients: 'allAttendees'
        },
        {
            '@odata.type':'#microsoft.graph.bookingReminder',
            message: 'Please be available to enjoy your lunch service.',
            offset: 'PT1H',
            'recipients@odata.type':'#microsoft.graph.bookingReminderRecipients',
            recipients: 'customer'
        },
        {
            '@odata.type':'#microsoft.graph.bookingReminder',
            message: 'Please check traffic for next cater.',
            offset: 'PT2H',
            'recipients@odata.type':'#microsoft.graph.bookingReminderRecipients',
            recipients: 'staff'
        }
    ],
    serviceId: '57da6774-a087-4d69-b0e6-6fb82c339976',
    serviceLocation: {
        '@odata.type':'#microsoft.graph.location',
        address: {
            '@odata.type':'#microsoft.graph.physicalAddress',
            city: 'Buffalo',
            countryOrRegion: 'USA',
            postalCode: '98052',
            postOfficeBox: null,
            state: 'NY',
            street: '123 First Avenue',
            'type@odata.type':'#microsoft.graph.physicalAddressType',
            type: null
        },
        coordinates: null,
        displayName: 'Customer location',
        locationEmailAddress: null,
        'locationType@odata.type':'#microsoft.graph.locationType',
        locationType: null,
        locationUri: null,
        uniqueId: null,
        'uniqueIdType@odata.type':'#microsoft.graph.locationUniqueIdType',
        uniqueIdType: null
    },
    serviceName: 'Catered bento',
    serviceNotes: 'Customer requires punctual service.',
    start: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-01T12:00:00.0000000+00:00',
        timeZone: 'UTC'
    }
};

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments')
    .version('beta')
    .post(bookingAppointment);

```