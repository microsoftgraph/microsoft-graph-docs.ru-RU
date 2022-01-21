---
title: тип ресурса identityProtectionRoot
description: Контейнер для свойств навигации для ресурсов microsoft Graph защиты удостоверений.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1d1ea31820743a0c132ee5f179b0917900a32e1a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161987"
---
# <a name="identityprotectionroot-resource-type"></a>тип ресурса identityProtectionRoot

Пространство имен: microsoft.graph

Контейнер для свойств навигации для ресурсов защиты Graph удостоверений.

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|riskDetections|[коллекция riskDetection](../resources/riskdetection.md)| Обнаружение рисков в Azure AD Identity Protection и связанных с этим сведений об обнаружении.|
|riskyUsers|[коллекция riskyUser](../resources/riskyuser.md)|Пользователи, помеченные как "под угрозой" в Azure AD Identity Protection. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProtectionRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProtectionRoot"
}
```

