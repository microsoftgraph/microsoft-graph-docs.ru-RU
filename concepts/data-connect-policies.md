---
title: Политики и лицензирование подключения к данным Microsoft Graph
description: Описаны поддерживаемые политики и способ назначения номеров SKU для доступа независимых поставщиков программного обеспечения в организации.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 2d592391222e39b3c6d4f6406205a99d72d32eb1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340680"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Политики и выставление счетов для подключения к данным Microsoft Graph

Подключение к данным Microsoft Graph осуществляется с помощью [управляемых приложений Azure](/azure/managed-applications/overview). С их помощью вы можете создать и развернуть решения в среде Azure. С помощью управляемых приложений вы можете поддерживать определенные политики Azure, обеспечивая клиентам более высокий доверительный уровень и комфортность при использовании приложений.

## <a name="policies"></a>Политики

Управляемые приложения Azure, созданные на основе данных Microsoft 365, поддерживают следующие политики Azure:

- [Служба хранилища Azure и требуемая политика ADLS 2-го поколения](/azure/storage/common/policy-reference)
- [Требуемая политика ADLS 1-го поколения](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Store 1-го и 2-го поколения используют разные политики, так как ADLS 2-го поколения реализует службу хранилища Azure.

После проверки состояния соответствия политике, выбранной во время публикации в Azure Marketplace, она применяется ко всем установленным экземплярам приложения. Все соответствующие выбранные политики отображаются для лиц, утверждающих данные, в рамках запроса данных. В случае нарушения соответствия политике происходит сбой в работе канала и прекращается извлечение данных.

## <a name="billing-for-microsoft-graph-data-connect"></a>Выставление счетов за подключение к данным Microsoft Graph

Счет будет связан с подпиской на Azure вашей Фабрики данных Azure. Цена в этой новой модели выставления счетов зависит от количества объектов Microsoft Graph, к которым вы обращаетесь. Дополнительные сведения о выставлении счетов см. на странице [Цены](https://azure.microsoft.com/pricing/details/graph-data-connect/).

Объекты каталога, за которые не выставляются счета:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>См. также

- [Политики служба хранилища Azure](/azure/storage/common/policy-reference)
- [Выставление счетов за подключение к данным Microsoft Graph](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [Управляемые приложения Azure](/azure/managed-applications/overview)
- [Выбор и фильтрация пользователей](data-connect-filtering.md)
- [Вопросы и ответы о подключении к данным](data-connect-faq.md)
