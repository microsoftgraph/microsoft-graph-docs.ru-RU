---
title: тип ресурса connectionInfo
description: Объект connectionInfo определяет сведения о подключении, используемые для связи с ресурсом.
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4c00cf41bd89deebf4b1453cb4f7389094e3dcb8
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242705"
---
# <a name="connectioninfo-resource-type"></a>тип ресурса connectionInfo

Пространство имен: microsoft.graph


Объект connectionInfo определяет локатор ресурсов, используемый для связи с ресурсом в Azure AD Entitlement Management.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|url|String|Конечная точка, используемая управлением правами для связи с ресурсом пакета доступа.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```


