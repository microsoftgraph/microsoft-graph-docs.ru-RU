---
title: Тип ресурса iosSingleSignOnSettings
description: операций ввода-вывода параметров проверки подлинности Kerberos для единого входа
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54c5656de6262692324cce8ab71a0e100672c050
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952673"
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





