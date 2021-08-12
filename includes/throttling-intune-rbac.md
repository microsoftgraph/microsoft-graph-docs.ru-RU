---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 7cb9d252a985c5c800bce56f8ff69cb03e1822d4ebecbc42819752f190c724db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196794"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-rbac-service-limits"></a>Ограничения службы Intune rbac

| Тип запроса | Ограничение на клиента для всех приложений | Ограничение на приложение по клиенту |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELETE, PATCH | 200 запросов за 20 секунд | 100 запросов за 20 секунд |
| Любой | 2000 запросов за 20 секунд | 1000 запросов за 20 секунд |

Указанные выше ограничения действуют для следующих ресурсов:  
deviceAndAppManagementRoleAssignment, deviceAndAppManagementRoleDefinition, resourceOperation, roleAssignment, roleDefinition, roleScopeTag, roleScopeTagAutoAssignment.
