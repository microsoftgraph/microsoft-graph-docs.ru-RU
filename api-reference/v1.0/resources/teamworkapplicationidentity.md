---
title: тип ресурса teamworkApplicationIdentity
description: Представляет приложение в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 78f5a4c681cae391037c6dc73d7d102d94dda6ce9c349fe6d5eeeed3fd9f3d8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249120"
---
# <a name="teamworkapplicationidentity-resource-type"></a>тип ресурса teamworkApplicationIdentity

Пространство имен: microsoft.graph

Представляет приложение **в** Microsoft Teams. `teamworkApplicationIdentity` используется для представления ботов и исходяющих веб-@mentioned в сообщениях.


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationIdentityType|teamworkApplicationIdentityType| Тип ссылаемого приложения. Возможные значения: `aadApplication` `bot` , , , , , `tenantBot` `office365Connector` и `outgoingWebhook` `unknownFutureValue` .|
|displayName|String|Унаследованный от [удостоверения](../resources/identity.md). Отображение имени приложения. Необязательно.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID приложения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

