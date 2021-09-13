---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8688bd9435766bfafe33b1e371f3a0812a7b4ce7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59096321"
---
# <a name="create-devicecategory"></a>Создание объекта deviceCategory

Пространство имен: microsoft.graph

> **Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).

## <a name="prerequisites"></a>Предварительные условия

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp; &nbsp; **Адаптация** | DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
| &nbsp; &nbsp; **Адаптация** | DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a>Заголовки запроса

|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса

В теле запроса добавьте представление объекта deviceCategory в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|
|**Обборка**|
|description|String|Необязательное описание категории устройств.|
|displayName|String|Отображаемое имя категории устройств.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```









