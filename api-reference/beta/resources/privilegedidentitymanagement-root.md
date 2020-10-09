---
title: Служба Privileged Identity Management
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory и ролями ресурсов Azure.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a29fca2d7bb94c87b17f1713088d36b1897ab38f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401619"
---
# <a name="privileged-identity-management"></a>Управление привилегированными пользователями

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Служба Privileged Identity Management (PIM) в Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) позволяет контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им. Сюда входит доступ к ресурсам в Azure AD, ресурсам Azure и другим службам Microsoft Online Services, таким как Microsoft 365 или Microsoft Intune. В Microsoft Graph предусмотрены интерфейсы API, которые можно использовать для управления ролями Azure AD и ролями ресурсов Azure.

- [Интерфейсы API для ролей Azure AD](privilegedidentitymanagement-directory.md)
- [Интерфейсы API для ролей ресурсов Azure](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> Этот API для управления ролями Azure AD будет изменяться с июня по ноябрь 2019 года для соответствия пространству имен и соглашению для [интерфейсов API ресурсов Azure](privilegedidentitymanagement-resources.md). Служба Azure AD PIM станет ресурсом в соответствии с соглашением о ресурсах Azure. Если это изменение непосредственно повлияет на ваш клиент, заполните [форму изменения интерфейса API Graph для Azure AD PIM](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u), чтобы получить дополнительные сведения, поддержку и возможность запланировать время для этого изменения API.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->