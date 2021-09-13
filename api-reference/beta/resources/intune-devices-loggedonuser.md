---
title: тип ресурса loggedOnUser
description: Вход в систему пользователя
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed949ddabbc38420054be2c7d03613bf1a5f0660
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095341"
---
# <a name="loggedonuser-resource-type"></a>тип ресурса loggedOnUser

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вход в систему пользователя

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Пользовательский id|
|lastLogOnDateTime|DateTimeOffset|Время даты входа пользователя в систему|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```



