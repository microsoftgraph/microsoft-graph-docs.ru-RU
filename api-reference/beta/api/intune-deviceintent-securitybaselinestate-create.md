---
title: Создание Секуритибаселинестате
description: Создание нового объекта Секуритибаселинестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f481bc5a3fa5e58017a671fe2fed43baa4c30af1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522526"
---
# <a name="create-securitybaselinestate"></a>Создание Секуритибаселинестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .

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
POST /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Секуритибаселинестате в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Секуритибаселинестате.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|Секуритибаселинетемплатеид|String|Идентификатор шаблона базовой безопасности|
|displayName|String|Отображаемое имя базового плана безопасности|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



