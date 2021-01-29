---
title: Тип ресурса userRegistrationFeatureCount
description: Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 0a0ad3758a74e057fa5539d3d913dd1735c88854
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052618"
---
# <a name="userregistrationfeaturecount-resource-type"></a>Тип ресурса userRegistrationFeatureCount

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет количество пользователей, зарегистрированных или способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|feature|authenticationMethodFeature|Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля. Возможные значения: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.|
|userCount|Int64|Количество пользователей.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
