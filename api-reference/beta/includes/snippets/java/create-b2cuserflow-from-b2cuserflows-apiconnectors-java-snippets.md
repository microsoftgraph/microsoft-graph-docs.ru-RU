---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 825f2708f0ee76d67d07f7fc6d17329ffebc7003
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844244"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.id = "UserFlowWithAPIConnector";
b2cIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2cIdentityUserFlow.userFlowTypeVersion = 1;
UserFlowApiConnectorConfiguration apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
IdentityApiConnector postFederationSignup = new IdentityApiConnector();
postFederationSignup.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/apiConnectors/{id}"));
apiConnectorConfiguration.postFederationSignup = postFederationSignup;
IdentityApiConnector postAttributeCollection = new IdentityApiConnector();
postAttributeCollection.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/apiConnectors/{id}"));
apiConnectorConfiguration.postAttributeCollection = postAttributeCollection;
b2cIdentityUserFlow.apiConnectorConfiguration = apiConnectorConfiguration;

graphClient.identity().b2cUserFlows()
    .buildRequest()
    .post(b2cIdentityUserFlow);

```