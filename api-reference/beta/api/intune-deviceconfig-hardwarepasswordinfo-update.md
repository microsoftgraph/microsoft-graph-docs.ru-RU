---
title: Обновление hardwarePasswordInfo
description: Обновление свойств объекта hardwarePasswordInfo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ddf665416159661ee7cf512565822146c3343ae5
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348431"
---
# <a name="update-hardwarepasswordinfo"></a>Обновление hardwarePasswordInfo

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/hardwarePasswordInfo/{hardwarePasswordInfoId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)

В следующей таблице показаны свойства, необходимые при создании [hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для информации о аппаратном пароле|
|serialNumber|String|Серийный номер устройства|
|currentPassword|Строка|Текущий пароль устройства|
|previousPasswords|Коллекция String|Список предыдущих паролей устройств|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwarePasswordInfo/{hardwarePasswordInfoId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "serialNumber": "Serial Number value",
  "currentPassword": "Current Password value",
  "previousPasswords": [
    "Previous Passwords value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "id": "418e4bb4-4bb4-418e-b44b-8e41b44b8e41",
  "serialNumber": "Serial Number value",
  "currentPassword": "Current Password value",
  "previousPasswords": [
    "Previous Passwords value"
  ]
}
```




