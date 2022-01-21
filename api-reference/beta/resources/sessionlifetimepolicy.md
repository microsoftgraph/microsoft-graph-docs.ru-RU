---
title: тип ресурса sessionlifetimepolicy
description: Описывает политики срока службы сеанса Azure AD, применяемые к событию входного знака.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9da2ea66c726d48fa3b0a34c168debd16dbd8713
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137282"
---
# <a name="sessionlifetimepolicy-resource-type"></a>тип ресурса sessionlifetimepolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает политики срока службы сеанса Azure AD, применяемые к событию входного знака. 

Дополнительные сведения об управлении сеансами с условным доступом в Azure AD см. в документации по управлению сеансами [условного доступа.](/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|expirationRequirement|expirationRequirement|Если политика управления сеансами условного доступа требовала от пользователя проверки подлинности в этом случае регистрации, в этом поле описывается тип политики, требуемой проверки подлинности. Возможные значения: `rememberMultifactorAuthenticationOnTrustedDevices`, `tenantTokenLifetimePolicy`, `audienceTokenLifetimePolicy`, `signInFrequencyPeriodicReauthentication`, `ngcMfa`, `signInFrequencyEveryTime`, `unknownFutureValue`.|
|подробные|Строка|Сведения о политике управления сеансами условного доступа, применимой к входу.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sessionLifetimePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sessionLifetimePolicy",
  "expirationRequirement": "String",
  "detail": "String"
}
```

