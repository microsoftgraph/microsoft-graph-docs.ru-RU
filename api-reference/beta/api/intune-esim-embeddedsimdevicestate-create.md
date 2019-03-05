---
title: Создание Ембеддедсимдевицестате
description: Создание нового объекта Ембеддедсимдевицестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d7ad1aa42f0cdeec9390d518491a02af346207b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175257"
---
# <a name="create-embeddedsimdevicestate"></a>Создание Ембеддедсимдевицестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Ембеддедсимдевицестате в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Ембеддедсимдевицестате.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор состояния встроенного SIM-устройства. Созданное системой значение, назначаемое при создании.|
|createdDateTime|DateTimeOffset|Время создания встроенного состояния SIM-устройства. Созданная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения состояния внедренного SIM-устройства. Обновленная сторона службы.|
|lastSyncDateTime|DateTimeOffset|Время последнего возврата встроенного SIM-устройства. Обновленная сторона службы.|
|УниверсалинтегратедЦиркуиткардидентифиер|String|Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.|
|deviceName|String|Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо|
|userName|String|Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).|
|state|[Ембеддедсимдевицестатевалуе](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Состояние операции профиля, примененной к устройству. Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|Статедетаилс|String|Строковое описание состояния подготовки.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```




