---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f172c0497c055b30876e491d41292c89fa0fa2f9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inviteParticipantsOperation = {
  participants: [
    {
      @odata.type: "#microsoft.graph.invitationParticipantInfo",
      replacesCallId: "a7ebfb2d-871e-419c-87af-27290b22e8db",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        user: {
          @odata.type: "#microsoft.graph.identity",
          id: "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          displayName: "string"
        }
      }
    },
    {
      @odata.type: "#microsoft.graph.invitationParticipantInfo",
      replacesCallId: "a7ebfb2d-871e-419c-87af-27290b22e8db",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        user: {
          @odata.type: "#microsoft.graph.identity",
          id: "1e126418-44a0-4a94-a6f8-0efe1ad71acb",
          displayName: "string"
        }
      }
    }
  ],
  clientContext: "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
};

let res = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/invite')
    .post(inviteParticipantsOperation);

```