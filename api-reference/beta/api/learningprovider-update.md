---
title: Обновление learningProvider
description: Обновление свойств объекта learningProvider.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: ac9ced68d3e3bad6ac794a6641bd98997ceb7633
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883411"
---
# <a name="update-learningprovider"></a>Обновление learningProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [learningProvider](../resources/learningprovider.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|LearningProvider.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /employeeExperience/learningProviders/{learningProviderId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя, отображаемое в Viva Обучение. Обязательный.|
|isEnabled|Boolean|Состояние поставщика. Необязательный элемент.|
|loginWebUrl|String|URL-адрес проверки подлинности для доступа к курсам для поставщика. Необязательный элемент.|
|longLogoWebUrlForDarkTheme|String|Длинный URL-адрес логотипа для темного режима, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|
|longLogoWebUrlForLightTheme|String|Длинный URL-адрес логотипа для светлого режима, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|
|squareLogoWebUrlForDarkTheme|String|URL-адрес квадратного логотипа для темного режима, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|
|squareLogoWebUrlForLightTheme|String|URL-адрес квадратного логотипа для режима освещения, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `204 No Content` отклика в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_learningprovider"
}
-->
``` http
PATCH /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70
Content-Type: application/json

{
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": false,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

