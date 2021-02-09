---
title: Создание windowsFeatureUpdateCatalogItem
description: Создание объекта windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc6e1a2d9e6b5f30e00e1212e8513f1af2dec7e0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162408"
---
# <a name="create-windowsfeatureupdatecatalogitem"></a>Создание windowsFeatureUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укатите представление объекта windowsFeatureUpdateCatalogItem в JSON.

В следующей таблице показаны свойства, необходимые при создании объекта windowsFeatureUpdateCatalogItem.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|String|Отображаемого имени элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога. Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|version|String|Версия обновления функций|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и объект `201 Created` [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```




