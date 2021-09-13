---
title: Создание встроенныхSIMActivationCodePool
description: Создайте новый встроенный объектSIMActivationCodePool.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab5ca0aace5afcf9da898c212950e307fcc1ef57
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097007"
---
# <a name="create-embeddedsimactivationcodepool"></a>Создание встроенныхSIMActivationCodePool

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [встроенный объектSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для встроенного объектаSIMActivationCodePool.

В следующей таблице показаны свойства, необходимые при создании встроенногоSIMActivationCodePool.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор встроенного пула кодов активации SIM. Созданное в системе значение, назначенное при его создания.|
|displayName|String|Администратор определил имя встроенного пула кодов активации SIM-карты.|
|createdDateTime|DateTimeOffset|Время создания встроенного пула кодов активации SIM-карты. Сгенерированная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения встроенного пула кодов активации SIM-карты. Обновленная сторона службы.|
|activationCodes|[коллекция embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)|Коды активации, которые принадлежат этому пулу. Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для чтения кодов активации из Intune.|
|activationCodeCount|Int32|Общее количество кодов активации, которые относятся к этому пулу.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и встроенный `201 Created` [объектSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте отклика.

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
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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



