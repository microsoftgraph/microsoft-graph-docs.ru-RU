---
title: тип ресурса iosCredentialSingleSignOnExtension
description: Представляет профиль одноместного Sign-On типа учетных данных для устройств iOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d356b901f3fbc2d912c2d29c028c29d9aa083f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069168"
---
# <a name="ioscredentialsinglesignonextension-resource-type"></a>тип ресурса iosCredentialSingleSignOnExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль одноместного Sign-On типа учетных данных для устройств iOS.


Наследует [от iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|extensionIdentifier|Строка|Получает или задает пакетный ID расширения приложения, который выполняет SSO для указанных URL-адресов.|
|teamIdentifier|Строка|Получает или задает командный ID расширения приложения, которое выполняет SSO для указанных URL-адресов.|
|домены|Коллекция строк|Получает или задает список хостов или доменных имен, для которых расширение приложения выполняет SSO.|
|realm|String|Получает или задает имя области, чувствительной к делу, для этого профиля.|
|конфигурации|[коллекция keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Получает или задает список пар значений ключей, используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCredentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```



