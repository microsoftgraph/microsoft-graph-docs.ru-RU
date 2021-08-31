---
title: тип ресурса groupPolicyUploadedLanguageFile
description: Объект представляет XML-файл ADML (язык административных шаблонов), загруженный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 015e2dc7372ecb2cec607b3e7c6a4aab940f5267
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794092"
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



