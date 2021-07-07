---
title: 'updatableAsset: unenrollAssets'
description: Unenroll updatableAsset resources from update management by the deployment service.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 8f32ca029e94da476eb1b6c491057a3d4343b523
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317191"
---
# <a name="updatableasset-unenrollassets"></a>updatableAsset: unenrollAssets
Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from update management by the deployment service.

Вы также можете использовать метод [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) для разгрузки активов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|WindowsUpdates.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/unenrollAssets
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|Категория обновлений для службы для остановки управления. Поддерживает подмножество значений **для updateCategory.** Возможные значения: `feature` .|
|assets|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Список **ресурсов updatableAsset** для отката от управления обновлениями службой для данного **обновленияCategory**.|



## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

