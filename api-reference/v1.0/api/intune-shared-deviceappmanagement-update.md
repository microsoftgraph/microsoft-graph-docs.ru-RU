---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f97316e06cec39cd0aeb1b22d6142925d81b77ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259369"
---
# <a name="update-deviceappmanagement"></a>Обновление объекта deviceAppManagement

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).  Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|**Подключение**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLanguage|String|Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса. Региональные параметры, относящиеся к стране или региону. Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий). Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166. Например, en-US для английского (США) — это определенный региональный стандарт.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле отклика.

## <a name="example-request"></a>Пример запроса

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a>Пример ответа

Объект Response, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



