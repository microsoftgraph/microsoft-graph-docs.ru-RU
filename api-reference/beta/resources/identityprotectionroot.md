---
title: тип ресурса identityProtectionRoot
description: Контейнер для свойств навигации для ресурсов microsoft Graph защиты удостоверений.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 90b8de67f24c650f1a4f6832979f5d669f9af57e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519468"
---
# <a name="identityprotectionroot-resource-type"></a>тип ресурса identityProtectionRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для свойств навигации для [ресурсов защиты Graph удостоверений](identityprotection-overview.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|riskDetections|[коллекция riskDetection](../resources/riskdetection.md)| Обнаружение рисков в Azure AD Identity Protection и связанных с этим сведений об обнаружении.|
|riskyUsers|[коллекция riskyUser](../resources/riskyuser.md)|Пользователи, помеченные как "под угрозой" в Azure AD Identity Protection. |
|riskyServicePrincipals| [коллекция riskyServicePrincipal](riskyserviceprincipal.md) | Директора служб Azure AD, которые находятся под угрозой. |
|servicePrincipalRiskDetections| [коллекция servicePrincipalRiskDetection](serviceprincipalriskdetection.md) | Представляет сведения о обнаруженных в клиенте Azure AD основных службах, которые могут быть обнаружены в опасности.|

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

