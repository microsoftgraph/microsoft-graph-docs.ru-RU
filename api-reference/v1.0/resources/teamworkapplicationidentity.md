---
title: тип ресурса teamworkApplicationIdentity
description: Представляет приложение в Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: af3f0205bf53137791414c2e4777877220ed6ca5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113527"
---
# <a name="teamworkapplicationidentity-resource-type"></a>тип ресурса teamworkApplicationIdentity

Пространство имен: microsoft.graph

Представляет приложение **в** Microsoft Teams. `teamworkApplicationIdentity` используется для представления ботов и исходяющих веб-@mentioned в сообщениях.


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationIdentityType|teamworkApplicationIdentityType| Тип ссылаемого приложения. Возможные значения: `aadApplication` `bot` , , , , , `tenantBot` `office365Connector` и `outgoingWebhook` `unknownFutureValue` .|
|displayName|String|Унаследованный от [удостоверения](../resources/identity.md). Отображение имени приложения. Необязательное.|
|id|Строка|Унаследованный от [удостоверения](../resources/identity.md). ID приложения.|

## <a name="relationships"></a>Отношения
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

