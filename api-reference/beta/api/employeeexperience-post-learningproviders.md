---
title: Создание learningProvider
description: Создайте объект learningProvider.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 40655e18f4fe22b3417f9ef2166538810ae36de4
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883383"
---
# <a name="create-learningprovider"></a>Создание learningProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [learningProvider](../resources/learningprovider.md) и зарегистрируйте его в Viva Обучение с помощью указанного отображаемого имени и логотипов для разных тем.

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
POST /employeeExperience/learningProviders
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [learningProvider](../resources/learningprovider.md) в формате JSON.

При создании **learningProvider** можно указать следующие свойства.

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

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [learningProvider](../resources/learningprovider.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_learningprovider_from_"
}
-->
``` http
POST /employeeExperience/learningProviders 
Content-Type: application/json

{
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": true,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningProvider"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders/$entity",
    "id": "ba9790ef-21d5-4c17-808c-acda55230253",
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": true,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```

