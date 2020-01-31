---
title: Управление доступом на основе ролей в Microsoft Intune
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые определяют управление доступом на основе ролей (RBAC) для организации клиента и управляют им.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: a43efe3a1c881eb014a075f30906dab79c7be13d
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636527"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="5d233-103">Управление доступом на основе ролей в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5d233-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="5d233-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d233-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d233-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d233-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d233-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d233-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d233-107">Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.</span><span class="sxs-lookup"><span data-stu-id="5d233-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="5d233-108">Следующие ресурсы Graph помогут в управлении доступом на основе ролей в Intune:</span><span class="sxs-lookup"><span data-stu-id="5d233-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="5d233-109">Данные назначенной роли для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="5d233-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="5d233-110">Назначение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="5d233-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="5d233-111">Определение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="5d233-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="5d233-112">Несколько приложений RBAC</span><span class="sxs-lookup"><span data-stu-id="5d233-112">Rbac application multiple</span></span>](intune-rbac-rbacapplicationmultiple.md)
- [<span data-ttu-id="5d233-113">Действие ресурса</span><span class="sxs-lookup"><span data-stu-id="5d233-113">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="5d233-114">Операция ресурса</span><span class="sxs-lookup"><span data-stu-id="5d233-114">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="5d233-115">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="5d233-115">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="5d233-116">Тип области назначения ролей</span><span class="sxs-lookup"><span data-stu-id="5d233-116">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="5d233-117">Определение ролей</span><span class="sxs-lookup"><span data-stu-id="5d233-117">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="5d233-118">Управление ролями</span><span class="sxs-lookup"><span data-stu-id="5d233-118">Role management</span></span>](intune-rbac-rolemanagement.md)
- [<span data-ttu-id="5d233-119">Разрешение роли</span><span class="sxs-lookup"><span data-stu-id="5d233-119">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="5d233-120">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="5d233-120">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="5d233-121">Автоматическое назначение тега области применения роли</span><span class="sxs-lookup"><span data-stu-id="5d233-121">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)
