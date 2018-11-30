---
title: Обновление sideLoadingKey
description: Обновление свойства объекта sideLoadingKey.
ms.openlocfilehash: 5c9071a47726f602fcd07fd47341c70f7b4b2f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080527"
---
# <a name="update-sideloadingkey"></a>Обновление sideLoadingKey

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойства объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .

В следующей таблице показаны свойства, которые необходимы для создания [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Со стороны загрузка уникальный идентификатор ключа.|
|value|String|Со стороны загрузки ключ значение — значение 5 x 5, разделенных hiphens.|
|displayName|String|Со стороны загрузка ключа имя, отображаемое для администраторов для ИТ-специалистов.|
|описание|String|Со стороны загрузки ключ описание, отображаемое для администраторов для ИТ-специалистов.|
|totalActivation|Int32|Со стороны загрузки ключ общее активация отображаются для администраторов для ИТ-специалистов.|
|lastUpdatedDateTime|String|Со стороны загрузки ключ обновлен Дата последнего отображаются для администраторов для ИТ-специалистов.|



## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) объекта в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 193

{
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





