---
title: тип ресурса resourceSpecificPermission
description: Представляет разрешения, используемые для авторизации приложения для прямого доступа к данным для определенного экземпляра ресурса
author: psignoret
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc1cd89ba26629b59c83fdd6b626cb280f69eaab
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63376390"
---
# <a name="resourcespecificpermission-resource-type"></a>тип ресурса resourceSpecificPermission

Пространство имен: microsoft.graph

Представляет разрешения, используемые для авторизации приложения для прямого доступа к данным для определенного экземпляра ресурса, например чата или группы. Например, разрешение ChannelMessage.Read.Group с определенными ресурсами позволяет приложению Microsoft Teams для чтения сообщений канала одной группы. 

Разрешения на использование ресурсов поддерживаются только для Teams приложений, которые могут получать доступ к определенным чатам и группам с помощью API microsoft Graph. Подробные сведения см. [в материале Resource-specific consent for Teams apps](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описывает уровень доступа, который представляет разрешение, определенное для ресурсов.|
|displayName|Строка|Имя отображения для разрешения, определенного для ресурсов.|
|id|GUID|Уникальный идентификатор разрешения приложения, определенного для ресурсов.|
|isEnabled|Boolean|Указывает, включено ли разрешение.|
|value|String|Значение разрешения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceSpecificPermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceSpecificPermission",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "value": "String"
}
```
