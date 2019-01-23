---
title: Тип ресурса iosSingleSignOnSettings
description: операций ввода-вывода параметров проверки подлинности Kerberos для единого входа
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421321"
---
# <a name="iossinglesignonsettings-resource-type"></a>Тип ресурса iosSingleSignOnSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

операций ввода-вывода параметров проверки подлинности Kerberos для единого входа

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список идентификаторов приложения, которые могут использовать это имя входа. Если это поле указан, имя входа применяется ко всем приложениям на устройстве. Эта коллекция может содержать не более 500 элементов.|
|allowedUrls|Коллекция String|Список URL-адресов HTTP для соответствия для использования этим именем входа. С помощью операций ввода-вывода 9.0 или более поздней версии могут быть использованы подстановочные знаки.|
|displayName|String|Отображаемое имя параметры входа в систему на получающей устройства.|
|kerberosPrincipalName|String|Имя участника Kerberos. Если этот параметр не указан, пользователю предлагается ввести один во время установки профиля.|
|kerberosRealm|String|Имя сферы Kerberos. С учетом регистра.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




