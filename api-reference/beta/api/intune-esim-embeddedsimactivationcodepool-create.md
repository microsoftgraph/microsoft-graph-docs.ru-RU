---
title: Создание embeddedSIMActivationCodePool
description: Создание нового объекта embeddedSIMActivationCodePool.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2d84230049c7b1f96756ac104557c5d8648c6a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394028"
---
# <a name="create-embeddedsimactivationcodepool"></a>Создание embeddedSIMActivationCodePool

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .

## <a name="prerequisites"></a>Предварительные требования
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
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта embeddedSIMActivationCodePool.

В следующей таблице показаны свойства, которые необходимы для создания embeddedSIMActivationCodePool.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для внедренных пула кода активации диспетчера установки. Значение, назначенное при создании создаваемый системой.|
|displayName|String|Имя группы внедренных диспетчера установки активации кода определенные администратором.|
|createdDateTime|DateTimeOffset|Время создания внедренных пула кода активации диспетчера установки. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения внедренного пула кода активации диспетчера установки. Обновление со стороны службы.|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) коллекции|Коды активации, которые относятся к этот пул. Это свойство навигации использовать для активации кодов Intune, но не может использоваться для чтения из Intune коды активации.|
|activationCodeCount|Int32|Общее число коды активации, которые относятся к этот пул.|



## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```




