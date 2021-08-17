---
title: тип ресурса customSubjectAlternativeName
description: Определение настраиваемого альтернативного имени субъекта
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 798c02446e7a3efbd5750fa914c4d14442114ef14b6713d25c0ee1559bbb30fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150473"
---
# <a name="customsubjectalternativename-resource-type"></a>тип ресурса customSubjectAlternativeName

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение настраиваемого альтернативного имени субъекта

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|sanType|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Настраиваемый тип SAN. Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|name|String|Пользовательское имя SAN|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




