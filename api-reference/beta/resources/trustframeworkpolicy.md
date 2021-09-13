---
title: trustFrameworkPolicy
description: В политике платформы доверия Azure AD B2C называются настраиваемые политики. В этом описаны операции, доступные для объекта trustFrameworkPolicy для клиента.
ms.localizationpriority: medium
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2f84f1ef4c391c81a720d5f0f76adae144e04677
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100521"
---
# <a name="trustframeworkpolicy-resource-type"></a>тип ресурса trustFrameworkPolicy

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет политику [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой](/azure/active-directory-b2c/active-directory-b2c-overview-custom)политикой) в Azure Active Directory [B2C](/azure/active-directory-b2c/active-directory-b2c-overview). Политика Trust Framework обеспечивает полный контроль над поездками пользователей. Используйте его для:

* Полностью настроить опытом регистрации и регистрации.
* Federate для любого поставщика удостоверений SAML, Open ID Подключение или поставщика удостоверений OAuth2.
* Интеграция с другими системами или хранилищами данных пользователей путем вызова конечных точек REST.
* Преобразование утверждений и настройка маркеров, выдающихся в приложение-участник.

Дополнительные сведения см. в [пользовательской политике в Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).

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


