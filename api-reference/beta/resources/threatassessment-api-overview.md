---
title: Использование API оценки угроз Microsoft Graph
description: Microsoft Graph позволяет приложению получить авторизованный доступ к данным оценки угроз организации.
localization_priority: Priority
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5360633155347b752866615e7635c811f3f1f30c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519787"
---
# <a name="use-the-microsoft-graph-threat-assessment-api"></a>Использование API оценки угроз Microsoft Graph

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

API оценки угроз Microsoft Graph позволяет организациям оценивать угрозу, возникшую для любого пользователя в клиенте. Благодаря этому пользователи могут сообщать в корпорацию Майкрософт о полученной нежелательной почте, фишинговых URL-адресах и вредоносных вложениях. Результат проверки политики и результат повторного сканирования может помочь администраторам клиента понять заключение сканирования угроз и настроить политику организации.

## <a name="authorization"></a>Авторизация

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Укажите разрешения, необходимые для доступа к оценке угроз, на портале Azure Active Directory (Azure AD). Дополнительные сведения см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference) и разделе [Разрешения для оценки угроз](/graph/permissions-reference#threat-assessment-permissions).

## <a name="common-use-cases"></a>Основные варианты использования

API оценки угроз Microsoft Graph предоставляет методы для перечисления, создания и получения запросов на оценку угроз, а также получения результатов оценки.

| Варианты использования | Ресурсы REST | См. также |
|:----------|:---------------|:---------|
| Перечисление, создание и получение запросов на оценку угроз | [threatAssessmentRequest](../resources/threatassessmentrequest.md)<br> [mailAssessmentRequest](../resources/mailAssessmentRequest.md)<br> [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)<br> [fileAssessmentRequest](../resources/fileAssessmentRequest.md)<br> [urlAssessmentRequest](../resources/urlAssessmentRequest.md)<br> | [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md)<br> [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md)<br> [Перечисление объектов threatAssessmentRequest](../api/informationprotection-list-threatassessmentrequests.md) |
| Получение результатов оценки угроз | [threatAssessmentResult](../resources/threatassessmentresult.md) | [Получение объекта threatAssessmentResult](../api/threatassessmentrequest-get.md#example-5-expand-threat-assessment-results-for-a-request)|

## <a name="next-steps"></a>Дальнейшие действия

Ресурсы оценки угроз и API Microsoft Graph открывают новые способы взаимодействия с пользователями и контроля их работы. Дополнительные сведения:

- Изучите подробнее [методы](../resources/threatassessmentrequest.md#methods), [свойства](../resources/threatassessmentrequest.md#properties) и [отношения](../resources/threatassessmentrequest.md#relationships) ресурсов [запросов на оценку угроз](../resources/threatassessmentrequest.md) и [результатов оценки угроз](../resources/threatAssessmentResult.md).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
