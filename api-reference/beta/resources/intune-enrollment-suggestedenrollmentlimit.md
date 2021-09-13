---
title: тип ресурса suggestedEnrollmentLimit
description: Предлагаемый ресурсEnrollmentLimit представляет рекомендуемый лимит регистрации при учете типа регистрации.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fca3ed6ad1d885fd01bc1aa313253a46b9acb4d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054340"
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



