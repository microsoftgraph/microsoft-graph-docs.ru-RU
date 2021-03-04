---
title: trustFrameworkPolicy
description: В политике платформы доверия Azure AD B2C называются настраиваемые политики. В этом описаны операции, доступные для объекта trustFrameworkPolicy для клиента.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8bb9fc598613d48ac6b9bb34aa02d24872e6300
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442742"
---
# <a name="trustframeworkpolicy-resource-type"></a>тип ресурса trustFrameworkPolicy

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет политику [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой](/azure/active-directory-b2c/active-directory-b2c-overview-custom)политикой) в Azure Active [Directory B2C.](/azure/active-directory-b2c/active-directory-b2c-overview) Политика Trust Framework обеспечивает полный контроль над поездками пользователей. Используйте его для:

* Полностью настроить опытом регистрации и регистрации.
* Federate к любому поставщику удостоверений SAML, Open ID Connect или поставщику удостоверений OAuth2.
* Интеграция с другими системами или хранилищами данных пользователей путем вызова конечных точек REST.
* Преобразование утверждений и настройка маркеров, выдающихся в приложение-участник.

Дополнительные сведения см. в [пользовательских политиках в Azure Active Directory B2C.](/azure/active-directory-b2c/active-directory-b2c-overview-custom)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание trustFrameworkPolicy](../api/trustframework-post-trustframeworkpolicy.md)|trustFrameworkPolicy|Создание нового trustFrameworkPolicy.|
|[Get trustFrameworkPolicy](../api/trustframeworkpolicy-get.md) |trustFrameworkPolicy|Чтение свойств существующего trustFrameworkPolicy.|
|[Список trustFrameworkPolicies](../api/trustframework-list-trustframeworkpolicies.md)|коллекция trustFrameworkPolicy|Список всех trustFrameworkPolicies, настроенных в клиенте.|
|[Обновление или создание trustFrameworkPolicy](../api/trustframework-put-trustframeworkpolicy.md)|Нет|Обновление существующего trustFrameworkPolicy.|
|[Удаление trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|Нет|Удаление существующего trustFrameworkPolicy.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|ID политики.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a>См. также

- [схема trustFrameworkPolicy](/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений о элементах схемы.
- [trustFrameworkPolicy.xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)


