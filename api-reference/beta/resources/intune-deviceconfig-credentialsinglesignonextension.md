---
title: тип ресурса credentialSingleSignOnExtension
description: Представляет профиль единого Sign-On типа учетных данных.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a90f6c3027a25c58204adf3ab5b5dbb32e4be6464896f28834f0eb9001e1d51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54203136"
---
# <a name="credentialsinglesignonextension-resource-type"></a>тип ресурса credentialSingleSignOnExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль единого Sign-On типа учетных данных.


Наследует [от singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|extensionIdentifier|Строка|Получает или задает пакетный ID расширения приложения, который выполняет SSO для указанных URL-адресов.|
|teamIdentifier|Строка|Получает или задает командный ID расширения приложения, которое выполняет SSO для указанных URL-адресов.|
|домены|Коллекция String|Получает или задает список хостов или доменных имен, для которых расширение приложения выполняет SSO.|
|realm|String|Получает или задает имя области, чувствительной к делу, для этого профиля.|
|конфигурации|[коллекция keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Получает или задает список пар значений ключей, используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```




