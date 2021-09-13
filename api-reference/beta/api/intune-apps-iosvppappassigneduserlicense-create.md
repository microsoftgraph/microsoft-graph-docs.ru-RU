---
title: Создание iosVppAppAssignedUserLicense
description: Создайте новый объект iosVppAppAssignedUserLicense.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51b61ed901692e01aba39b6323128c05f359c8a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126480"
---
# <a name="create-iosvppappassigneduserlicense"></a>Создание iosVppAppAssignedUserLicense

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта iosVppAppAssignedUserLicense.

В следующей таблице показаны свойства, необходимые при создании iosVppAppAssignedUserLicense.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|String|Адрес электронной почты пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|Имя участника-пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```



