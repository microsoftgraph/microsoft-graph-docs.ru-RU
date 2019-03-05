---
title: Обновление Виндовсманажементапфеалссуммари
description: Обновление свойств объекта Виндовсманажементапфеалссуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 764549ee57bc3ab3a2a1e0c2db9c6ac16309b85d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155967"
---
# <a name="update-windowsmanagementapphealthsummary"></a>Обновление Виндовсманажементапфеалссуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [Виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта сводки работоспособности приложения управления Windows.|
|Хеалсидевицекаунт|Int32|Работоспособное число устройств.|
|Унхеалсидевицекаунт|Int32|Неработоспособное число устройств.|
|unknownDeviceCount|Int32|Количество неИзвестных устройств.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```




