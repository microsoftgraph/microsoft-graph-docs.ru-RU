---
title: Тип перечисления keyStorageProviderOption
description: Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f3a8169b4bb6cd2357f02aa7fec89ba640780f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946555"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="43805-103">Тип перечисления keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="43805-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="43805-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43805-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43805-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43805-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43805-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43805-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43805-107">Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).</span><span class="sxs-lookup"><span data-stu-id="43805-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="43805-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="43805-108">Members</span></span>
|<span data-ttu-id="43805-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="43805-109">Member</span></span>|<span data-ttu-id="43805-110">Значение</span><span class="sxs-lookup"><span data-stu-id="43805-110">Value</span></span>|<span data-ttu-id="43805-111">Описание</span><span class="sxs-lookup"><span data-stu-id="43805-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43805-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="43805-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="43805-113">0</span><span class="sxs-lookup"><span data-stu-id="43805-113">0</span></span>|<span data-ttu-id="43805-114">Импорта для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — импорт поставщика хранилища КЛЮЧЕЙ программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="43805-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="43805-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="43805-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="43805-116">1</span><span class="sxs-lookup"><span data-stu-id="43805-116">1</span></span>|<span data-ttu-id="43805-117">Импорт для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — не удается.</span><span class="sxs-lookup"><span data-stu-id="43805-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="43805-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="43805-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="43805-119">2</span><span class="sxs-lookup"><span data-stu-id="43805-119">2</span></span>|<span data-ttu-id="43805-120">Импорт Passport для работы поставщика хранилища КЛЮЧЕЙ Если доступно, в противном случае — ошибка.</span><span class="sxs-lookup"><span data-stu-id="43805-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="43805-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="43805-121">useSoftwareKsp</span></span>|<span data-ttu-id="43805-122">3</span><span class="sxs-lookup"><span data-stu-id="43805-122">3</span></span>|<span data-ttu-id="43805-123">Импорт на программное обеспечение поставщика хранилища КЛЮЧЕЙ.</span><span class="sxs-lookup"><span data-stu-id="43805-123">Import to Software KSP.</span></span>|





