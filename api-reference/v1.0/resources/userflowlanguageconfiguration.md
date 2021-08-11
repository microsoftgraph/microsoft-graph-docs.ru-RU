---
title: тип ресурса userFlowLanguageConfiguration
description: Позволяет потоку пользователей поддерживать несколько языков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b40df72429bdc1b23bbb9426ae9b9f78154257491ba3c715d57c0804b226df98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221154"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>тип ресурса userFlowLanguageConfiguration

Пространство имен: microsoft.graph

Позволяет потоку пользователей поддерживать использование нескольких языков.

Для [Azure Active Directory](/azure/active-directory/external-identities/user-flow-customize-language)потоков пользователей можно использовать только встроенные языки, предоставляемые Корпорацией Майкрософт. Потоки пользователей Azure Active Directory, определяющие язык и строки, показанные пользователям во время поездок, которые вы настраивали с помощью пользовательских потоков.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Эти объекты представляют язык, доступный в потоке пользователей.|
|[Список defaultPages](../api/userflowlanguageconfiguration-list-defaultpages.md)|[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages. Представляет путь пользователя по умолчанию в потоке пользователей.|
|[Переопределения списка](../api/userflowlanguageconfiguration-list-overridespages.md)|[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages. Представляет настраиваемый интерфейс для пользовательского путешествия в потоке пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор языка. Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.|
|isEnabled|Boolean|Указывает, включен ли язык в потоке пользователей.|
|displayName|String|Отображаемая языковая фамилия. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|defaultPages|[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Коллекция страниц с контентом по умолчанию, отображаемым в потоке пользователей для указанного языка. Эта коллекция не позволяет вносить какие-либо изменения.|
|overridesPages|[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Коллекция страниц с переопределениями сообщений для отображения в потоке пользователей для указанного языка. Эта коллекция позволяет изменять только содержимое страницы, любые другие изменения не допускаются (создание или удаление страниц).|

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
