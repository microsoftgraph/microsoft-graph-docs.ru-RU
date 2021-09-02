---
title: тип ресурса suggestedEnrollmentLimit
description: Предлагаемый ресурсEnrollmentLimit представляет рекомендуемый лимит регистрации при учете типа регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7c01f21a85a84d9cddff349913e596b32793df5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817364"
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



