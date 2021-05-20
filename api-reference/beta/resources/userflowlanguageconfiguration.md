---
title: тип ресурса userFlowLanguageConfiguration
description: Объект userFlowsLanguageConfiguration позволяет потоку пользователей поддерживать настройку нескольких языков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aa83d85725cbef54229cdc92246fb83888697166
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547150"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>тип ресурса userFlowLanguageConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка языка потоков пользователей — это функция, которая позволяет заданный поток пользователей поддерживать настройку нескольких языков, от всех встроенных языков до настраиваемого языка.

Для Azure Active Directory потоки пользователей [B2C](/azure/active-directory-b2c/user-flow-language-customization#supported-languages)можно использовать встроенные языки или предоставить языковые настройки для языка, который в настоящее время не встроен по умолчанию. Для [Azure Active Directory](/azure/active-directory/external-identities/user-flow-customize-language)потоков пользователей можно использовать только встроенные языки, предоставляемые Корпорацией Майкрософт. Потоки пользователей Azure Active Directory B2C и Azure Active Directory поддерживают настройку языка и строк, показанных пользователям во время поездок, настроенных с потоками пользователей.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Эти объекты представляют язык, доступный в потоке пользователей.|
|[Удаление userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|Нет|Удаляет настраиваемый [объект userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Эти объекты представляют язык, доступный в потоке пользователей, и из потока пользователей Azure AD B2C можно удалить только настраиваемый язык.|
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
