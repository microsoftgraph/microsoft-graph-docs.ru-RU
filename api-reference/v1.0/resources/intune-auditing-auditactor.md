---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
ms.openlocfilehash: ae784e5ad16b54c553dadaa75ed5a849b692211f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025312"
---
# <a name="auditactor-resource-type"></a>Тип ресурса auditActor

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, содержащий свойства субъекта аудита.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|String|Тип субъекта.|
|userPermissions|Коллекция строк|Список разрешений пользователей во время аудита.|
|applicationId|String|ИД приложения AAD.|
|applicationDisplayName|String|Имя приложения.|
|userPrincipalName|String|Имя участника-пользователя (UPN).|
|servicePrincipalName|String|Имя субъекта-службы (SPN).|
|ipAddress|String|IP-адрес.|
|userId|String|ИД пользователя.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```



