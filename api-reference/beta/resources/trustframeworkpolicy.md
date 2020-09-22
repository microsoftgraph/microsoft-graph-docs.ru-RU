---
title: трустфрамеворкполици
description: В политике Azure AD B2C Trust Framework называются пользовательскими политиками. В этом разделе описываются операции, доступные в объекте Трустфрамеворкполици для клиента.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bad5d8cfa6d9b53c4023bb89eabd74436ab7dacd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057950"
---
# <a name="trustframeworkpolicy-resource-type"></a>Тип ресурса Трустфрамеворкполици

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет политику [платформы доверия](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой политикой](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) в [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview). Политика инфраструктуры доверия предоставляет полный контроль над путешествием пользователей. Используйте его для:

* Полностью настройте вход и вход в систему.
* Федерацию на любой поставщик удостоверений SAML, Open ID Connect или OAuth2.
* Интеграция с другими системами или хранилищами пользовательских данных путем вызова конечных точек REST.
* Преобразование утверждений и настройка маркеров, выданных приложению проверяющей стороны.

Для получения дополнительных сведений см. [настраиваемые политики в Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание Трустфрамеворкполици](../api/trustframework-post-trustframeworkpolicy.md)|трустфрамеворкполици|Создание нового Трустфрамеворкполици.|
|[Получение Трустфрамеворкполици](../api/trustframeworkpolicy-get.md) |трустфрамеворкполици|Чтение свойств существующего Трустфрамеворкполици.|
|[Список ТрустфрамеворкполиЦиес](../api/trustframework-list-trustframeworkpolicies.md)|Коллекция Трустфрамеворкполици|Список всех ТрустфрамеворкполиЦиес, настроенных в клиенте.|
|[Обновление или создание Трустфрамеворкполици](../api/trustframework-put-trustframeworkpolicy.md)|Нет|Обновление существующего Трустфрамеворкполици.|
|[Удаление Трустфрамеворкполици](../api/trustframeworkpolicy-delete.md)|Нет|Удаление существующего Трустфрамеворкполици.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор политики.|

## <a name="json-representation"></a>Представление в формате JSON

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

- [схема трустфрамеворкполици](/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений об элементах схемы.
- [Трустфрамеворкполици. xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)


