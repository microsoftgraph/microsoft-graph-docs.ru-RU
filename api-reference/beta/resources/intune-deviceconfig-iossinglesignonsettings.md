---
title: Тип ресурса iosSingleSignOnSettings
description: операций ввода-вывода параметров проверки подлинности Kerberos для единого входа
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17c2e100f9762334173ca6ca7049d1e5933f8616
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841064"
---
# <a name="iossinglesignonsettings-resource-type"></a>Тип ресурса iosSingleSignOnSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

операций ввода-вывода параметров проверки подлинности Kerberos для единого входа
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список идентификаторов приложения, которые могут использовать это имя входа. Если это поле указан, имя входа применяется ко всем приложениям на устройстве. Эта коллекция может содержать не более 500 элементов.|
|allowedUrls|Коллекция String|Список URL-адресов HTTP для соответствия для использования этим именем входа. С помощью операций ввода-вывода 9.0 или более поздней версии могут быть использованы подстановочные знаки.|
|displayName|Строка|Отображаемое имя параметры входа в систему на получающей устройства.|
|kerberosPrincipalName|Строка|Имя участника Kerberos. Если этот параметр не указан, пользователю предлагается ввести один во время установки профиля.|
|kerberosRealm|Строка|Имя сферы Kerberos. С учетом регистра.|

## <a name="relationships"></a>Связи
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





