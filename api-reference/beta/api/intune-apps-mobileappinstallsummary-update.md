---
title: Обновление mobileAppInstallSummary
description: Обновление свойств объекта mobileAppInstallSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb69e7db1cf5f85a0655ee931f5d98778d9a98d1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025134"
---
# <a name="update-mobileappinstallsummary"></a>Обновление mobileAppInstallSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
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

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)

В следующей таблице показаны свойства, необходимые при создании [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|installedDeviceCount|Int32|Количество устройств, успешно установленных в этом приложении.|
|failedDeviceCount|Int32|Количество устройств, которые не смогли установить это приложение.|
|notApplicableDeviceCount|Int32|Количество устройств, которые не применимы для этого приложения.|
|notInstalledDeviceCount|Int32|Количество устройств, на которые не установлено это приложение.|
|pendingInstallDeviceCount|Int32|Количество устройств, которые были уведомлены об установке этого приложения.|
|installedUserCount|Int32|Число пользователей, устройства которых успешно установили это приложение.|
|failedUserCount|Int32|Число пользователей, у них есть 1 или более устройств, которые не смогли установить это приложение.|
|notApplicableUserCount|Int32|Число пользователей, устройства которых не были применимы к этому приложению.|
|notInstalledUserCount|Int32|Число пользователей с 1 или более устройствами, которые не установили это приложение.|
|pendingInstallUserCount|Int32|Число пользователей с 1 или более устройствами, которые были уведомлены об установке этого приложения, и имеют 0 устройств с ошибками.|



## <a name="response"></a>Ответ
В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) в тексте ответа.

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



