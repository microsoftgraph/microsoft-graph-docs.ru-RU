---
title: Тип ресурса userFlowLanguageConfiguration
description: Объект userFlowsLanguageConfiguration позволяет пользовательскому потоку поддерживать настройку нескольких языков.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9c963fcb7f22af34de92d0ad1c9a472974e346f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159796"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>Тип ресурса userFlowLanguageConfiguration

Пространство имен: microsoft.graph

Пользовательские потоки настройки языка — это функция, которая позволяет заданным пользовательским потокам поддерживать настройку нескольких языков— от всех встроенных языков до настраиваемых.

Для потоков пользователей [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages)можно использовать встроенные языки или настроить язык для языка, который в настоящее время не встроен по умолчанию. Для [потоков пользователей Azure Active Directory](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)можно использовать только встроенные языки, предоставляемые корпорацией Майкрософт. Потоки пользователей для Azure Active Directory B2C и Azure Active Directory поддерживают настройку языка и строк, которые показываются пользователям при настройке потоков пользователей.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Чтение свойств и связей объекта [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Эти объекты представляют язык, доступный в пользовательском потоке.|
|[Удаление userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|Нет|Удаляет пользовательский [объект userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Эти объекты представляют язык, доступный в пользовательском потоке, и только пользовательский язык можно удалить из пользовательского потока Azure AD B2C.|
|[Список defaultPages](../api/userflowlanguageconfiguration-list-defaultpages.md)|[Коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages. Представляет пользовательский путь по умолчанию в пользовательском потоке.|
|[Список overridesPages](../api/userflowlanguageconfiguration-list-overridespages.md)|[Коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages. Представляет пользовательский интерфейс для пользовательского пути в пользовательском потоке.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор языка. Это поле является тегом языка, совместимым с [RFC 5646,](https://tools.ietf.org/html/rfc5646) и должно быть документированным ИД языка.|
|isEnabled|Boolean|Указывает, включен ли язык в пользовательском потоке.|
|displayName|String|Отображаемого имени языка. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|defaultPages|[Коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Коллекция страниц с содержимым по умолчанию для отображения в пользовательском потоке для указанного языка. Эта коллекция не допускает каких-либо изменений.|
|overridesPages|[Коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)|Коллекция страниц с переопределениями сообщений для отображения в пользовательском потоке для указанного языка. Эта коллекция позволяет изменять только содержимое страницы, любые другие изменения не допускаются (создание или удаление страниц).|

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
