---
title: Создание Клаудпкдевицеимаже
description: Отправьте настраиваемый образ ОС, который вы можете подготовить к работе на облачных компьютерах.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4cbfb96f6adf70a197b3d648d1bddb4cd405a1c9
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563473"
---
# <a name="create-cloudpcdeviceimage"></a>Создание Клаудпкдевицеимаже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) . Отправьте настраиваемый образ ОС, который вы можете подготовить к работе на облачных компьютерах.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Клаудпк. ReadWrite. ALL|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                |
| :------------ | :------------------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя изображения.|
|саурцеимажересаурцеид|String|Идентификатор исходного ресурса изображения в Azure. Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.компуте/имажес/{имаженаме}".|
|operatingSystem|String|Операционная система изображения. Пример: Windows 10 Корпоративная.|
|осбуилднумбер|String|Версия сборки ОС образа. Пример: 1909.|
|version|String|Версия изображения. Например: 0.0.1, 1.5.13.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcdeviceimage_from_cloudpcdeviceimage"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 508

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
  "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
  "status": "pending",
  "statusDetails": null
}
```
