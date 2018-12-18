---
title: Тип перечисления keyStorageProviderOption
description: Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).
author: tfitzmac
ms.openlocfilehash: 7923dd5c4b8a09d834d29b65928430828f3dafac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342219"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="9bb37-103">Тип перечисления keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="9bb37-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="9bb37-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9bb37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bb37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bb37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bb37-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9bb37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bb37-107">Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).</span><span class="sxs-lookup"><span data-stu-id="9bb37-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="9bb37-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9bb37-108">Members</span></span>
|<span data-ttu-id="9bb37-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9bb37-109">Member</span></span>|<span data-ttu-id="9bb37-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9bb37-110">Value</span></span>|<span data-ttu-id="9bb37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bb37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb37-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="9bb37-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="9bb37-113">0</span><span class="sxs-lookup"><span data-stu-id="9bb37-113">0</span></span>|<span data-ttu-id="9bb37-114">Импорта для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — импорт поставщика хранилища КЛЮЧЕЙ программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="9bb37-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="9bb37-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="9bb37-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="9bb37-116">1</span><span class="sxs-lookup"><span data-stu-id="9bb37-116">1</span></span>|<span data-ttu-id="9bb37-117">Импорт для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — не удается.</span><span class="sxs-lookup"><span data-stu-id="9bb37-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="9bb37-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="9bb37-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="9bb37-119">2</span><span class="sxs-lookup"><span data-stu-id="9bb37-119">2</span></span>|<span data-ttu-id="9bb37-120">Импорт Passport для работы поставщика хранилища КЛЮЧЕЙ Если доступно, в противном случае — ошибка.</span><span class="sxs-lookup"><span data-stu-id="9bb37-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="9bb37-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="9bb37-121">useSoftwareKsp</span></span>|<span data-ttu-id="9bb37-122">3</span><span class="sxs-lookup"><span data-stu-id="9bb37-122">3</span></span>|<span data-ttu-id="9bb37-123">Импорт на программное обеспечение поставщика хранилища КЛЮЧЕЙ.</span><span class="sxs-lookup"><span data-stu-id="9bb37-123">Import to Software KSP.</span></span>|





