---
title: Создание chromeOSOnboardingSettings
description: Создайте новый объект chromeOSOnboardingSettings.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a7200f79be8647c127135ae471a23d155f4d3d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59112995"
---
# <a name="create-chromeosonboardingsettings"></a>Создание chromeOSOnboardingSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса поставляем представление JSON для объекта chromeOSOnboardingSettings.

В следующей таблице показаны свойства, необходимые при создании chromeOSOnboardingSettings.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id ChromebookTenant|
|ownerUserPrincipalName|String|OwnerUserPrincipalName ChromebookTenant|
|onboardingStatus|[onboardingStatus](../resources/intune-chromebooksync-onboardingstatus.md)|OnboardingStatus ChromebookTenant. Возможные значения: `unknown`, `inprogress`, `onboarded`, `failed`.|
|lastModifiedDateTime|DateTimeOffset|LastModifiedDateTime ChromebookTenant|
|lastDirectorySyncDateTime|DateTimeOffset|LastDirectorySyncDateTime в ChromebookTenant|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "0344255d-255d-0344-5d25-44035d254403",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```



