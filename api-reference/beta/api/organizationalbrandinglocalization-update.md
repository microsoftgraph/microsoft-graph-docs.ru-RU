---
title: Обновление организационнойБрандингЛокализации
description: Обновление свойств объекта organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9a07607894dac7ce62a4ac4e74fd5c5ec056a17e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777468"
---
# <a name="update-organizationalbrandinglocalization"></a>Обновление организационнойБрандингЛокализации
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [организационнойbrandingLocalization](../resources/organizationalbrandinglocalization.md) для определенной локализации.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Только типы данных Stream, включая **backgroundLogo и** **backgroundImage,** обновляются с помощью метода PUT. Чтобы обновить типы данных String, включая **signInPageText** и **usernameHintText,** используйте метод PATCH. В том же запросе нельзя обновлять типы потоков с другими типами данных.

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
PUT /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса *поставляют только* значения для свойств, которые должны быть обновлены. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.

В следующей таблице указаны свойства, которые можно обновить. 

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый `#FFFFFF` . |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
| signInPageText | Строка | Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Разрешены типы PNG или JPEG размером не более 240 x 240 пикселей и размером не более 10 КБ. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
| usernameHintText | Строка | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране входной записи. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-setting-bannerlogo-for-the-fr-fr-localization-using-put"></a>Пример 1. Настройка **bannerLogo** для локализации fr-FR с помощью PUT

Следующий запрос обновляет логотип баннера для локализации fr-FR.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR/bannerLogo
Content-Type: image/jpeg

<Image>
```


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-the-backgroundcolor-and-signinpagetext-for-the-fr-fr-localization-using-patch"></a>Пример 2. Обновление backgroundColor и signInPageText для локализации fr-FR с помощью PATCH

Следующий запрос обновляет логотип баннера для `fr-FR` локализации.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization6"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "Welcome to Contoso France"
}
```


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-a-default-branding-value-with-a-blank-string"></a>Пример 3. Переопределение значения брендинга по умолчанию с пустой строкой

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization7"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "signInPageText": "Welcome to Contoso France.",
    "usernameHintText":" "
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

После этого запроса имя пользователяHintText для локализации будет пустым, а не наследуется значение от объекта `fr-FR` брендинга по умолчанию.
