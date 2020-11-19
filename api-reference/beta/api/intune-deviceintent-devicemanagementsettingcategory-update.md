---
title: Обновление Девицеманажементсеттингкатегори
description: Обновление свойств объекта Девицеманажементсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b3889af273c6a0c80a7437994c660bcbb9b0ce1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229627"
---
# <a name="update-devicemanagementsettingcategory"></a>Обновление Девицеманажементсеттингкатегори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор категории|
|displayName|String|Имя категории|
|хасрекуиредсеттинг|Boolean|Категория содержит параметры, необходимые для верхнего уровня|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




