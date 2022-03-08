---
title: тип ресурса customExtensionClientConfiguration
description: Параметры подключения HTTP, которые определяют, как долго Azure AD может ждать ответа из логического приложения, прежде чем оно отключит подключение. Поддерживается только timeoutInMilliseconds.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c04e53560aecc3e41978b569e42d993477eca87
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339673"
---
# <a name="customextensionclientconfiguration-resource-type"></a>тип ресурса customExtensionClientConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры подключения HTTP, которые определяют, как долго Azure AD может ждать ответа из логического приложения, прежде чем оно отключит подключение. **Поддерживается только timeoutInMilliseconds**.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|timeoutInMilliseconds|Int32|Максимальная продолжительность в миллисекунд, которую Azure AD будет ждать ответа от логического приложения, прежде чем оно отключит подключение. Допустимый диапазон между миллисекундами `200` `2000` . Продолжительность по умолчанию .`1000`|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customExtensionClientConfiguration",
  "timeoutInMilliseconds": "Integer"
}
```

