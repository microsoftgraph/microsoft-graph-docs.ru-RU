---
title: Обновление oemWarrantyInformationOnboarding
description: Обновление свойств объекта oemWarrantyInformationOnboarding.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 24647d27cdebfe0d74500323694d38d132e60846
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292448"
---
# <a name="update-oemwarrantyinformationonboarding"></a>Обновление oemWarrantyInformationOnboarding

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/oemWarrantyInformationOnboarding/{oemWarrantyInformationOnboardingId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .

В следующей таблице показаны свойства, необходимые при создании [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для статуса гарантии OEM. Это свойство доступно только для чтения.|
|oemName|String|Имя OEM. Это свойство доступно только для чтения.|
|enabled|Boolean|Указывает, включен ли гарантийный запрос для данного OEM. Это свойство доступно только для чтения.|
|доступен|Логическое|Указывает, доступен ли API гарантии. Это свойство доступно только для чтения.|



## <a name="response"></a>Отклик
В случае успешной `200 OK` работы этот метод возвращает код ответа и обновленный [объект oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/oemWarrantyInformationOnboarding/{oemWarrantyInformationOnboardingId}
Content-type: application/json
Content-length: 148

{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "oemName": "Oem Name value",
  "enabled": true,
  "available": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 197

{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "id": "55491425-1425-5549-2514-495525144955",
  "oemName": "Oem Name value",
  "enabled": true,
  "available": true
}
```




