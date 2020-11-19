---
title: Тип ресурса Граупполициуплоадедлангуажефиле
description: Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf5bef8faadac012df13a8a31cfaac3a5dc94ed2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298108"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>Тип ресурса Граупполициуплоадедлангуажефиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|fileName|String|Имя файла загруженного файла ADML.|
|лангуажекоде|String|Код языка загруженного файла ADML.|
|содержимое|Binary|Содержимое отправленного файла ADML.|
|id|String|Ключ объекта.|
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




