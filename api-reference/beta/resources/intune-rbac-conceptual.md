---
title: Управление доступом на основе ролей в Microsoft Intune
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые определяют управление доступом на основе ролей (RBAC) для организации клиента и управляют им.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 86f0e3c08bf1180969085d49f715cc6c52d8aec4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527571"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="72d30-103">Управление доступом на основе ролей в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="72d30-103">Role-based access control in Microsoft Intune</span></span>

<span data-ttu-id="72d30-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72d30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72d30-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72d30-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72d30-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d30-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72d30-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72d30-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72d30-108">Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.</span><span class="sxs-lookup"><span data-stu-id="72d30-108">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="72d30-109">Следующие ресурсы Graph помогут в управлении доступом на основе ролей в Intune:</span><span class="sxs-lookup"><span data-stu-id="72d30-109">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="72d30-110">Данные назначенной роли для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="72d30-110">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="72d30-111">Назначение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="72d30-111">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="72d30-112">Определение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="72d30-112">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="72d30-113">Действие ресурса</span><span class="sxs-lookup"><span data-stu-id="72d30-113">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="72d30-114">Операция ресурса</span><span class="sxs-lookup"><span data-stu-id="72d30-114">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="72d30-115">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="72d30-115">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="72d30-116">Тип области назначения ролей</span><span class="sxs-lookup"><span data-stu-id="72d30-116">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="72d30-117">Определение ролей</span><span class="sxs-lookup"><span data-stu-id="72d30-117">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="72d30-118">Разрешение роли</span><span class="sxs-lookup"><span data-stu-id="72d30-118">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="72d30-119">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="72d30-119">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="72d30-120">Автоматическое назначение тега области применения роли</span><span class="sxs-lookup"><span data-stu-id="72d30-120">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)
