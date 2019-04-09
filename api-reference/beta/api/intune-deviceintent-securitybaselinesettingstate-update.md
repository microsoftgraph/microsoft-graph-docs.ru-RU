---
title: Обновление Секуритибаселинесеттингстате
description: Обновление свойств объекта Секуритибаселинесеттингстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3295cb35fbc9002f458a60d6f1b78a2ef380126b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524584"
---
# <a name="update-securitybaselinesettingstate"></a>Обновление Секуритибаселинесеттингстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .

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
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [Секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта|
|settingName|String|Имя параметра, о котором сообщается|
|state|[Секуритибаселинекомплианцестате](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Состояние соответствия параметру базового уровня безопасности. Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|Сеттингкатегорид|String|Идентификатор категории параметров, к которой относится этот параметр|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "798e520d-520d-798e-0d52-8e790d528e79",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```



