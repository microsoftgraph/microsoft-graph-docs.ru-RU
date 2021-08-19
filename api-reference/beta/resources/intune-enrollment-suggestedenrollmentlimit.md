---
title: тип ресурса suggestedEnrollmentLimit
description: Предлагаемый ресурсEnrollmentLimit представляет рекомендуемый лимит регистрации при учете типа регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7595aa2ab614a7c9abb0ac9c76c4b05fda1288eea7b11c24b2b1932a1265a321
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197942"
---
# <a name="suggestedenrollmentlimit-resource-type"></a>тип ресурса suggestedEnrollmentLimit

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предлагаемый ресурсEnrollmentLimit представляет рекомендуемый лимит регистрации при учете типа регистрации.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|suggestedDailyLimit|Int32|Рекомендуемый лимит регистрации в течение дня|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```




