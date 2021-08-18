---
title: тип ресурса groupPolicyUploadedLanguageFile
description: Объект представляет XML-файл ADML (язык административных шаблонов), загруженный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c77b9f6fab6bbd1127aff4abc0176a9298f6e6a2955f69a2781c9f22f63069f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122364"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>тип ресурса groupPolicyUploadedLanguageFile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет XML-файл ADML (язык административных шаблонов), загруженный администратором.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|fileName|String|Имя файла загруженного ADML-файла.|
|languageCode|Строка|Языковой код загруженного ADML-файла.|
|содержимое|В двоичном формате|Содержимое загруженного ADML-файла.|
|id|Строка|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedLanguageFile",
  "fileName": "String",
  "languageCode": "String",
  "content": "binary",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




