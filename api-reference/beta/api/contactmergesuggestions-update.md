---
title: Обновление contactMergeSuggestions
description: Обновление свойств объекта contactMergeSuggestions.
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 582bf04e32f449d4dedd597451bdd14c8676a073
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339582"
---
# <a name="update-contactmergesuggestions"></a>Обновление contactMergeSuggestions
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [contactMergeSuggestions](../resources/contactmergesuggestions.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|User.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/settings/contactMergeSuggestions
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
|isEnabled|Boolean|`true` если функция слияния дублирующих контактов включена для пользователя; `false` если функция отключена. Значение по умолчанию: `true`.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `204 No Content` отклика, и значение обновляется в задней части.

## <a name="examples"></a>Примеры

В следующем примере обновляется **параметр конфиденциальности isEnabled** , чтобы отключить функцию слияния предложений с дублирующими контактами.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_contactmergesuggestions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/settings/contactMergeSuggestions
Content-Type: application/json

{
  "isEnabled": false
}
```


### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

<!-- {
  "blockType": "response",
  "name": "update_contactmergesuggestions"
}
-->
``` http
HTTP/1.1 204 No Content
```

