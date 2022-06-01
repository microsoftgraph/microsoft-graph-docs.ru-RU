---
title: Тип ресурса userRegistrationFeatureCount
description: Число пользователей, зарегистрированных или поддерживающих многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 609c8d30547093c19d93428a0c779687b93ae018
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820184"
---
# <a name="userregistrationfeaturecount-resource-type"></a>Тип ресурса userRegistrationFeatureCount

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет количество пользователей, зарегистрированных или поддерживающих Многофакторную идентификацию, Self-Service и проверку подлинности без пароля.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Функция|authenticationMethodFeature|Число пользователей, зарегистрированных или поддерживающих многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля. Возможные значения: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.|
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
