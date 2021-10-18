---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b6c6eadca68c8c41bc13b9aee3dd547ae1f7921
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450061"
---
# <a name="auditactor-resource-type"></a>Тип ресурса auditActor

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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



