---
title: Управление доступом на основе ролей в Microsoft Intune
description: 'Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.   '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cbbd04aacd80c8ad3c3082505ab052e2bdd65cbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924358"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="737b4-103">Управление доступом на основе ролей в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="737b4-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="737b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="737b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="737b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="737b4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="737b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="737b4-107">Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.</span><span class="sxs-lookup"><span data-stu-id="737b4-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="737b4-108">Следующие ресурсы Graph помогут в управлении доступом на основе ролей в Intune:</span><span class="sxs-lookup"><span data-stu-id="737b4-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="737b4-109">Устройства и приложения управления, назначенные роли идентификаторы</span><span class="sxs-lookup"><span data-stu-id="737b4-109">Device and app management assigned role ids</span></span>](intune-rbac-deviceandappmanagementassignedroleids.md)
- [<span data-ttu-id="737b4-110">Назначение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="737b4-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="737b4-111">Определение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="737b4-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="737b4-112">Действие ресурса</span><span class="sxs-lookup"><span data-stu-id="737b4-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="737b4-113">Операция ресурса</span><span class="sxs-lookup"><span data-stu-id="737b4-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="737b4-114">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="737b4-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="737b4-115">Тип области назначения ролей</span><span class="sxs-lookup"><span data-stu-id="737b4-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="737b4-116">Определение ролей</span><span class="sxs-lookup"><span data-stu-id="737b4-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="737b4-117">Разрешение роли</span><span class="sxs-lookup"><span data-stu-id="737b4-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="737b4-118">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="737b4-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
