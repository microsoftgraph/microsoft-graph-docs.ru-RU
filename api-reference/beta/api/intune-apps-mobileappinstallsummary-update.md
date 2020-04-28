---
title: Обновление Мобилеаппинсталлсуммари
description: Обновление свойств объекта Мобилеаппинсталлсуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fab58b772d9cb9111c7676a08703dd7868d7d4cb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43414791"
---
# <a name="update-mobileappinstallsummary"></a>Обновление Мобилеаппинсталлсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|installedDeviceCount|Int32|Количество устройств, на которых успешно установлено это приложение.|
|failedDeviceCount|Int32|Количество устройств, которые не удалось установить это приложение.|
|notApplicableDeviceCount|Int32|Количество устройств, неприменимых к этому приложению.|
|notInstalledDeviceCount|Int32|Количество устройств, на которых не установлено это приложение.|
|пендингинсталлдевицекаунт|Int32|Количество устройств, которые были уведомлены об установке этого приложения.|
|installedUserCount|Int32|Количество пользователей, чьи устройства успешно выполнили установку этого приложения.|
|failedUserCount|Int32|Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.|
|notApplicableUserCount|Int32|Количество пользователей, чьи устройства были неприменимы к этому приложению.|
|notInstalledUserCount|Int32|Количество пользователей с 1 или больше устройств, которые не установили это приложение.|
|пендингинсталлусеркаунт|Int32|Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```



