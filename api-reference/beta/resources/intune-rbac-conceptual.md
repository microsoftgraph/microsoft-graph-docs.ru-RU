---
title: Управление доступом на основе ролей в Microsoft Intune
description: 'Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.   '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 4cdc5e875f698646288258fc225ad77f8c4c2ba8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395750"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="dc72e-103">Управление доступом на основе ролей в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="dc72e-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="dc72e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc72e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc72e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc72e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc72e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc72e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="dc72e-107">Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.</span><span class="sxs-lookup"><span data-stu-id="dc72e-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="dc72e-108">Следующие ресурсы Graph помогут в управлении доступом на основе ролей в Intune:</span><span class="sxs-lookup"><span data-stu-id="dc72e-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="dc72e-109">Устройства и приложения управления, назначенных сведения о роли</span><span class="sxs-lookup"><span data-stu-id="dc72e-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="dc72e-110">Назначение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="dc72e-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="dc72e-111">Определение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="dc72e-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="dc72e-112">Действие ресурса</span><span class="sxs-lookup"><span data-stu-id="dc72e-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="dc72e-113">Операция ресурса</span><span class="sxs-lookup"><span data-stu-id="dc72e-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="dc72e-114">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="dc72e-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="dc72e-115">Тип области назначения ролей</span><span class="sxs-lookup"><span data-stu-id="dc72e-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="dc72e-116">Определение ролей</span><span class="sxs-lookup"><span data-stu-id="dc72e-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="dc72e-117">Разрешение роли</span><span class="sxs-lookup"><span data-stu-id="dc72e-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="dc72e-118">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="dc72e-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
