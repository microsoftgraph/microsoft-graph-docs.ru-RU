---
title: тип ресурса appConsentApprovalRoute
description: Контейнер для базовых ресурсов, которые раскрывают API запроса на согласие приложения и функции. В настоящее время предоставляется только связь appConsentRequests.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb5e5c3c060c255d7c5154494cc0226031665e5f
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651040"
---
# <a name="appconsentapprovalroute-resource-type"></a>тип ресурса appConsentApprovalRoute

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для базовых ресурсов, которые раскрывают API запроса на согласие приложения и функции. В настоящее время предоставляется [только связь appConsentRequests.](appconsentrequest.md)

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|appConsentRequests|[коллекция appConsentRequest](../resources/appconsentrequest.md)| Коллекция объектов [userConsentRequest](../resources/userconsentrequest.md) для определенного приложения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentApprovalRoute",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentApprovalRoute"
}
```

