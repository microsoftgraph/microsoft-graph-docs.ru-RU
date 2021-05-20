---
title: пользовательFlowLanguageКонфигурация типа ресурса
description: Позволяет потоку пользователей поддерживать несколько языков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 556860eb77c4707f1d180b7924ae3126958a4799
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547206"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>пользовательFlowLanguageКонфигурация типа ресурса

Пространство имен: microsoft.graph

Позволяет потоку пользователей поддерживать использование нескольких языков.

Для [Azure Active Directory потоков пользователей,](/azure/active-directory/external-identities/user-flow-customize-language)вы можете использовать только встроенные языки, предоставляемые корпорацией Майкрософт. Потоки пользователей для Azure Active Directory поддержки, определяющей язык и строки, показанные пользователям по мере их настройки с потоками пользователей.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить userFlowLanguageКонфигурация](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Прочитайте свойства и отношения объекта [пользователяFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Эти объекты представляют собой язык, доступный в пользовательском потоке.|
|[Список по умолчаниюВеся](../api/userflowlanguageconfiguration-list-defaultpages.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция|Получите ресурсы userFlowLanguagePage из навигационного свойства defaultPages. Представляет путешествие пользователя по умолчанию в потоке пользователя.|
|[Список переопределяетВит Страницы](../api/userflowlanguageconfiguration-list-overridespages.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция|Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages. Представляет собой пользовательский интерфейс для путешествия пользователя в потоке пользователя.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор языка. Это поле соответствует тегу Language ID [RFC 5646](https://tools.ietf.org/html/rfc5646) и должно быть задокументированным идентификатором языка.|
|isEnabled|Boolean|Указывает, включен ли язык в потоке пользователя.|
|displayName|String|Название языка для отображения. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|по умолчаниюВееся|[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция|Сбор страниц с содержимым по умолчанию для отображения в пользовательском потоке для определенного языка. Эта коллекция не допускает каких-либо изменений.|
|переопределяет Страницы|[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция|Сбор страниц с переопределениями сообщений для отображения в пользовательском потоке для определенного языка. Эта коллекция позволяет изменять только содержимое страницы, любая другая модификация не допускается (создание или удаление страниц).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```
