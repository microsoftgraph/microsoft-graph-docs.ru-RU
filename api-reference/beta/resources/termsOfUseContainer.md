---
title: тип ресурса termsOfUseContainer
description: Контейнер для отношений, которые раскрывают условия использования API и его функций. В настоящее время предоставляет соглашения и отношения agreementAcceptances.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: bef1033ceea7056d52586054f4ba32f98953cbe0
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651792"
---
# <a name="termsofusecontainer-resource-type"></a>тип ресурса termsOfUseContainer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для отношений, которые раскрывают условия использования API и его функций. В настоящее время предоставляет [соглашения](agreement.md) и [отношения agreementAcceptances.](agreementacceptance.md)

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|agreementAcceptances|Коллекция [agreementAcceptance](agreementacceptance.md)| Представляет текущее состояние ответа пользователя на настраиваемые условия соглашения об использовании компании.|
|соглашения|[коллекция соглашений](agreement.md)|Представляет настраиваемые условия соглашения об использовании клиента, созданного и управляемого Azure Active Directory Azure AD.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsOfUseContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsOfUseContainer"
}
```

