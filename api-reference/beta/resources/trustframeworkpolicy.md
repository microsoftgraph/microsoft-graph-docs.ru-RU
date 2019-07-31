---
title: Трустфрамеворкполици
description: В политике Azure AD B2C Trust Framework называются пользовательскими политиками. В этом разделе описываются операции, доступные в объекте Трустфрамеворкполици для клиента.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f573b331b587db50019e71468ec98d0e746e3963
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964188"
---
# <a name="trustframeworkpolicy-resource-type"></a>Тип ресурса Трустфрамеворкполици

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет политику [платформы доверия](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой политикой](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) в [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview). Политика инфраструктуры доверия предоставляет полный контроль над путешествием пользователей. Используйте его для:

* Полностью настройте вход и вход в систему.
* Федерацию на любой поставщик удостоверений SAML, Open ID Connect или OAuth2.
* Интеграция с другими системами или хранилищами пользовательских данных путем вызова конечных точек REST.
* Преобразование утверждений и настройка маркеров, выданных приложению проверяющей стороны.

Для получения дополнительных сведений см. [настраиваемые политики в Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание Трустфрамеворкполици](../api/trustframework-post-trustframeworkpolicy.md)|Трустфрамеворкполици|Создание нового Трустфрамеворкполици.|
|[Получение Трустфрамеворкполици](../api/trustframeworkpolicy-get.md) |Трустфрамеворкполици|Чтение свойств существующего Трустфрамеворкполици.|
|[Список ТрустфрамеворкполиЦиес](../api/trustframework-list-trustframeworkpolicies.md)|Коллекция Трустфрамеворкполици|Список всех ТрустфрамеворкполиЦиес, настроенных в клиенте.|
|[Обновление или создание Трустфрамеворкполици](../api/trustframework-put-trustframeworkpolicy.md)|Нет|Обновление существующего Трустфрамеворкполици.|
|[Удаление Трустфрамеворкполици](../api/trustframeworkpolicy-delete.md)|Нет|Удаление существующего Трустфрамеворкполици.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор политики.|

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

- [схема трустфрамеворкполици](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений об элементах схемы.  
- [Трустфрамеворкполици. xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
