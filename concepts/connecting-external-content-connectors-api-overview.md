---
title: Работа с API соединителей
description: Обзор API соединителей Microsoft Graph
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 63e11b086592a46a4e519a2ab7c79c20d049213a
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52646296"
---
# <a name="working-with-the-connectors-api"></a><span data-ttu-id="52605-103">Работа с API соединителей</span><span class="sxs-lookup"><span data-stu-id="52605-103">Working with the connectors API</span></span>

<span data-ttu-id="52605-104">Соединители Microsoft Graph — это простой способ добавления внешних данных в Microsoft Graph и улучшения интеллектуальных технологий Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52605-104">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph and enhance Microsoft 365 intelligent experiences.</span></span> <span data-ttu-id="52605-105">Для интеграции со службами, которые недоступны в роли соединителей, созданных корпорацией Майкрософт, необходимо создать настраиваемый соединитель.</span><span class="sxs-lookup"><span data-stu-id="52605-105">You might want to build a custom connector to integrate with services that aren't available as connectors built by Microsoft.</span></span> <span data-ttu-id="52605-106">Чтобы создать настраиваемые соединители, используйте REST API соединителей Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52605-106">To build custom connectors, you use the Microsoft Graph connector REST APIs.</span></span>

![Изображение внешних данных, исходящих из разных соединителей Microsoft Graph](./images/connectors-images/api-overview.png)

<span data-ttu-id="52605-108">Используйте API Microsoft Graph, чтобы выполнять следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="52605-108">You can use the Microsoft Graph connectors API to:</span></span>

1. <span data-ttu-id="52605-109">Создание подключений к внешним данным и управление ими.</span><span class="sxs-lookup"><span data-stu-id="52605-109">Create and manage external data connections.</span></span>
2. <span data-ttu-id="52605-110">Определение и регистрация схем внешних типов данных.</span><span class="sxs-lookup"><span data-stu-id="52605-110">Define and register the schema of the external data type(s).</span></span>
3. <span data-ttu-id="52605-111">Запись элементов внешних данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52605-111">Ingest external data items into Microsoft Graph.</span></span>
4. <span data-ttu-id="52605-112">Синхронизация внешних групп.</span><span class="sxs-lookup"><span data-stu-id="52605-112">Sync external groups.</span></span>

<span data-ttu-id="52605-113">Дополнительные сведения об этих API можно найти в документации, представленной далее.</span><span class="sxs-lookup"><span data-stu-id="52605-113">To learn more details about these APIs, you can visit the documentation suggested next.</span></span>

## <a name="connections-api"></a><span data-ttu-id="52605-114">API подключений</span><span class="sxs-lookup"><span data-stu-id="52605-114">Connections API</span></span>

<span data-ttu-id="52605-115">Подключение — это логический контейнер для внешних данных, которыми вы можете управлять как единым целым.</span><span class="sxs-lookup"><span data-stu-id="52605-115">A connection is a logical container for your external data that you can manage as a single unit.</span></span>
<span data-ttu-id="52605-116">Дополнительную информацию о создании, обновлении и удалении подключений в Microsoft Graph можно найти в разделе [Управление подключениями](connecting-external-content-manage-connections.md).</span><span class="sxs-lookup"><span data-stu-id="52605-116">To learn more about how to create, update, and delete connections in the Microsoft Graph, visit the [Manage connection](connecting-external-content-manage-connections.md) section.</span></span>

## <a name="schema-api"></a><span data-ttu-id="52605-117">API схем</span><span class="sxs-lookup"><span data-stu-id="52605-117">Schema API</span></span>

<span data-ttu-id="52605-118">[Схема](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true) связей определяет, как ваше содержимое будет использоваться в различных интерфейсах Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52605-118">The connection [schema](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true) determines how your content will be used in various Microsoft 365 experiences.</span></span> <span data-ttu-id="52605-119">Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы.</span><span class="sxs-lookup"><span data-stu-id="52605-119">Schema is a flat list of all the properties you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="52605-120">Перед добавлением элементов в Microsoft Graph вы должны зарегистрировать схему.</span><span class="sxs-lookup"><span data-stu-id="52605-120">You must register the schema before ingesting items into Microsoft Graph.</span></span>

<span data-ttu-id="52605-121">Дополнительную информацию о регистрации схемы для подключения Microsoft Graph и его свойствах можно найти в разделе [Управление схемой](connecting-external-content-manage-schema.md).</span><span class="sxs-lookup"><span data-stu-id="52605-121">To learn more about how to register the schema for the Microsoft Graph connection, and its properties, visit the [Manage schema](connecting-external-content-manage-schema.md) section.</span></span>

## <a name="ingest-external-data-items"></a><span data-ttu-id="52605-122">Прием элементов внешних данных</span><span class="sxs-lookup"><span data-stu-id="52605-122">Ingest external data items</span></span>

<span data-ttu-id="52605-123">Соединители Microsoft Graph — это простой способ добавления внешних данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52605-123">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph.</span></span> <span data-ttu-id="52605-124">Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52605-124">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

<span data-ttu-id="52605-125">Дополнительные сведения о создании, обновлении и удалении элементов, добавленных приложением через соединители Microsoft Graph см. в разделе [Управление элементами](connecting-external-content-manage-items.md).</span><span class="sxs-lookup"><span data-stu-id="52605-125">To learn more about how to create, update, and delete items added by your application via Microsoft Graph connectors, visit the [Manage items](connecting-external-content-manage-items.md) section.</span></span>

## <a name="external-groups-api"></a><span data-ttu-id="52605-126">API внешних групп</span><span class="sxs-lookup"><span data-stu-id="52605-126">External groups API</span></span>

<span data-ttu-id="52605-127">Элементам во внешней службе может предоставляться или отказываться в доступе через ACL к различным типам групп, отличных от Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52605-127">Items in the external service can be granted or denied access via ACL to different types of non-Azure Active Directory groups.</span></span> <span data-ttu-id="52605-128">Например, элементы Salesforce могут иметь наборы разрешений и профили.</span><span class="sxs-lookup"><span data-stu-id="52605-128">For example, Salesforce items might have permission sets and profiles.</span></span> <span data-ttu-id="52605-129">Элементы ServiceNow могут иметь локальные группы.</span><span class="sxs-lookup"><span data-stu-id="52605-129">ServiceNow items might have local groups.</span></span> <span data-ttu-id="52605-130">При записи этих элементов в Microsoft Graph необходимо соблюдать эти ACL.</span><span class="sxs-lookup"><span data-stu-id="52605-130">When you ingest these items into Microsoft Graph, you need to honor these ACLs.</span></span>

<span data-ttu-id="52605-131">Вы можете использовать API внешних групп, чтобы настроить разрешения для внешних элементов, которые будут записаны в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52605-131">You can use the External groups API to set permissions on external items ingested into Microsoft Graph.</span></span> <span data-ttu-id="52605-132">[externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) представляет группу, отличную от Azure Active Directory или групповую конструкцию (например, бизнес-единицы, Teams и так далее) и определяет разрешения на содержимое во внешнем источнике данных.</span><span class="sxs-lookup"><span data-stu-id="52605-132">An [externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) represents a non-Azure Active Directory group or group-like construct (such as Business units, Teams, and so on) and determines permissions on the content in your external data source.</span></span>