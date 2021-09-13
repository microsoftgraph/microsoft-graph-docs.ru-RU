---
title: тип ресурса userFlowLanguageConfiguration
description: Позволяет потоку пользователей поддерживать несколько языков.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9af22f309ca7c93043d90ef8c0583686d7cf24f2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136322"
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
|id|Строка|Идентификатор языка. Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.|
|isEnabled|Boolean|Указывает, включен ли язык в потоке пользователей.|
|displayName|Строка|Отображаемая языковая фамилия. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Отношения

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
