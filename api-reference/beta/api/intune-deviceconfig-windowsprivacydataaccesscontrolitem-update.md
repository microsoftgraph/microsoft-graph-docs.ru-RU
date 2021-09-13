---
title: Обновление windowsPrivacyDataAccessControlItem
description: Обновление свойств объекта windowsPrivacyDataAccesssControlItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c9114c8a6b5c02d51d7bc5f221ca8df2b445d060
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103090"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a>Обновление windowsPrivacyDataAccessControlItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsPrivacyDataAccesssControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса устройте представление JSON для [объекта windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)

В следующей таблице показаны свойства, необходимые при создании [windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ WindowsPrivacyDataAccessControlItem.|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Это указывает уровень доступа к категории данных конфиденциальности, которой будет предоставлено указанное приложение. Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Это указывает на категорию данных конфиденциальности, к которой будет применяться определенный контроль доступа. Возможные значения: `notConfigured` `accountInfo` , , , , , `appsRunInBackground` , , , `calendar` `callHistory` , , `camera` `contacts` `diagnosticsInfo` `email` , `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` .|
|appPackageFamilyName|String|Имя семейства пакета приложения Windows. При наборе уровень доступа применяется к указанному приложению.|
|appDisplayName|String|Имя семейства пакета приложения Windows. При наборе уровень доступа применяется к указанному приложению.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```



