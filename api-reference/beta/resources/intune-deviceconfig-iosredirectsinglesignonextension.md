---
title: тип ресурса iosRedirectSingleSignOnExtension
description: Представляет профиль одноместного Sign-On типа перенаправления для устройств iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40ebc4a9fae68b47bc4558a17d97390fb00d577f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803008"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a>тип ресурса iosRedirectSingleSignOnExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль одноместного Sign-On типа перенаправления для устройств iOS.


Наследует [от iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|extensionIdentifier|Строка|Получает или задает пакетный ID расширения приложения, который выполняет SSO для указанных URL-адресов.|
|teamIdentifier|Строка|Получает или задает командный ID расширения приложения, которое выполняет SSO для указанных URL-адресов.|
|конфигурации|[коллекция keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Получает или задает список пар значений ключей, используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|
|urlPrefixes|Коллекция String|Один или несколько префиксов URL-адресов поставщиков удостоверений, от имени которых расширение приложения выполняет один вход. URL-адреса должны начинаться с http:// или https://. Все префиксы URL-адресов должны быть уникальными для всех профилей.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



